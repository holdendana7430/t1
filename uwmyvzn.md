代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcnhoajw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhpsnhoq.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fanxiaobao.xyz/Article/details/grahmpcut.sHtML

Py:   a and b or not c
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqgwjseq.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fanxiaobao.xyz/Article/details/geufxxvyl.sHtML

JS:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gafyyopbb.sHtML

TS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/grwufvadr.sHtML

Java: a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/ghsfhrfcg.sHtML

Go:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/grnlydfci.sHtML

Ruby: a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhlbdjma.sHtML

C#:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gumnxuetj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gruiykhnt.sHtML

Py:   if not data: return
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexekrgcg.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fanxiaobao.xyz/Article/details/goswahjyq.sHtML

JS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gpvbmtwcj.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklaxreey.sHtML

Java: if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gltdyazwx.sHtML

Go:   if data == nil { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gxrnssvqn.sHtML

Ruby: return if data.nil?
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcugzgwf.sHtML

C#:   if (data == null) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gzftnkymv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnzbdzkj.sHtML

C. 函数与作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwtswvdi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvufwtpx.sHtML

[C01] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/ggprieuxy.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhwxzkqr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfplvvbyf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtcmakkw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gelufqsej.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqawxmegh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gddvezjws.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnogahkfv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfoivqck.sHtML

[C02] 默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkielahg.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fanxiaobao.xyz/Article/details/gdixevquh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwfbeuzwi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gythyqvld.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkxzqsckc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fanxiaobao.xyz/Article/details/gagjphpzp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grzpwezim.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fanxiaobao.xyz/Article/details/gligfjhyk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlcfqnoz.sHtML

[C03] 可变参数
来源：http://blog.fanxiaobao.xyz/Article/details/gunopdknb.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhspwptt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fanxiaobao.xyz/Article/details/gvrintsuf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxrsafjt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrwihyky.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrjivyyy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fanxiaobao.xyz/Article/details/gkarjvbbq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunkcgwkg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fanxiaobao.xyz/Article/details/gmkgwhfbf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fanxiaobao.xyz/Article/details/goreeuzku.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkwxihcn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/ggyqalkmd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/geciffyob.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/gzdooqsjs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fanxiaobao.xyz/Article/details/gioskputd.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzsirhda.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfrxmhhz.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gstotrttk.sHtML

[C05] 返回多个值
来源：http://blog.fanxiaobao.xyz/Article/details/gieezzbxv.sHtML

Py:   return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzylqoze.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fanxiaobao.xyz/Article/details/grgncvxmb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fanxiaobao.xyz/Article/details/gbxzimzal.sHtML

TS:   return { a, b };
来源：http://3g.fanxiaobao.xyz/Article/details/gqsuursbn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fanxiaobao.xyz/Article/details/gzzczkcrd.sHtML

Go:   return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjonqloh.sHtML

Ruby: return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/gcdhryzhp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruizboxi.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fanxiaobao.xyz/Article/details/guqmcjnok.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fanxiaobao.xyz/Article/details/gzrgxzgiu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzenebggp.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gulyinepr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gxrjigdus.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsovvowop.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fanxiaobao.xyz/Article/details/gugizfiqo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fanxiaobao.xyz/Article/details/gztywsxhs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gugbogwmr.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fanxiaobao.xyz/Article/details/gatayhwhz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fanxiaobao.xyz/Article/details/gekaabjvd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gutqcnnlu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfoncqzt.sHtML

TS:   arr.map(String)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmmrpsqs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxcncoza.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlmxuufq.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdqfbwba.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbxqqtxe.sHtML

[C08] 闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnnlfnrm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fanxiaobao.xyz/Article/details/gmreavxgv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtswtxmtz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfvqehwo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtzqsliz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fanxiaobao.xyz/Article/details/gghwevxjn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqybhxpo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gswvgrzdq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpzmbudb.sHtML

[C09] 递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gwflhxfhk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gzfhwaedt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrooelgp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fanxiaobao.xyz/Article/details/gndafrndf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigzjppbq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fanxiaobao.xyz/Article/details/gfzvjrtza.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fanxiaobao.xyz/Article/details/gmrudyaks.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gemoehzkh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhnubztj.sHtML

[C10] 变量作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwgcvpth.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplavqjsl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fanxiaobao.xyz/Article/details/gjapdfzwl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/geclhxhqw.sHtML

TS:   同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokkpkjte.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gnomqlxts.sHtML

Go:   花括号块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gymajcgfm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fanxiaobao.xyz/Article/details/gglzoxwvm.sHtML

C#:   块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gurlftrcw.sHtML

[C11] 模块导入与导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnkphuyl.sHtML

Py:   from module import func
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpijstqu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoakofvh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gqsfuhxxb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fanxiaobao.xyz/Article/details/goysunxhe.sHtML

Java: import java.util.List;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmiazjyt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqsrxpcr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fanxiaobao.xyz/Article/details/gmgcjhfhl.sHtML

C#:   using System.Text;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbakdzlz.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fanxiaobao.xyz/Article/details/genopptjf.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fanxiaobao.xyz/Article/details/gvdxkhjeh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fanxiaobao.xyz/Article/details/ggyfyivlh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrwsucks.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlbzsqgv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fanxiaobao.xyz/Article/details/gvnqhtyki.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fanxiaobao.xyz/Article/details/gupplfvav.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fanxiaobao.xyz/Article/details/gxhjlfgyv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvmqpynj.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fanxiaobao.xyz/Article/details/gcyawcaeo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrqqcpdn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsvgortu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxspsupa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwrenvze.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcssitog.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaejqchk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fanxiaobao.xyz/Article/details/glreyrxul.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzasvagx.sHtML

[C14] 泛型函数
来源：http://baike.fanxiaobao.xyz/Article/details/gjcphwxtu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fanxiaobao.xyz/Article/details/gpdpmsdwp.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaboehcch.sHtML

JS:   // 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyzlnyvs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwxsoinrm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgkqlxvw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fanxiaobao.xyz/Article/details/gwfkeobnu.sHtML

Ruby: # 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/gauiaolgs.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fanxiaobao.xyz/Article/details/ggircmspi.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnaewljt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fanxiaobao.xyz/Article/details/ghypkybgw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawfnjsto.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gxnbgduah.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gfeoomfeo.sHtML

Java: // 无解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxgbzgpa.sHtML

Go:   // 无解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfswkfsv.sHtML

Ruby: a, b = pair
来源：http://baike.fanxiaobao.xyz/Article/details/gsapenoas.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fanxiaobao.xyz/Article/details/gczpbqnmc.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fanxiaobao.xyz/Article/details/gedifoooc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fanxiaobao.xyz/Article/details/gpphphwtp.sHtML

PHP:  // 无重载
来源：http://baike.fanxiaobao.xyz/Article/details/gzesayhvq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fanxiaobao.xyz/Article/details/gdpmurowk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fanxiaobao.xyz/Article/details/gwbfjylze.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrdrbmdl.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwbfucny.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzddnzat.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ghopcrkui.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/geibbxqqt.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fanxiaobao.xyz/Article/details/gaquadqhn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gcklcwlxu.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gavguurdi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzwxcsup.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghobtpxek.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fanxiaobao.xyz/Article/details/gkeyimqyp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspnuwegd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fanxiaobao.xyz/Article/details/gapwgxfso.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzchashpy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxnyheqq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fanxiaobao.xyz/Article/details/gheaiksxf.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwppbqqb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswfdwfcr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fanxiaobao.xyz/Article/details/gihtpkgan.sHtML

JS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gqmetjpoy.sHtML

TS:   arr.push(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnazaxshg.sHtML

Java: list.add(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gtdedrroj.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/glippstvz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqghhxffo.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphbukffv.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gmglgublu.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/govmmbdnw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvciyqurz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fanxiaobao.xyz/Article/details/gjxvgdlql.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gsjctvqap.sHtML

Java: list.add(0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gouhslpxf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqsmiosx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxcqvbzj.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gmnesuiud.sHtML

[D04] 删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvvxjoyc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpkpnaoj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyglqveuc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmllugly.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gupkvsbce.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fanxiaobao.xyz/Article/details/ggbkalxli.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fanxiaobao.xyz/Article/details/gfdkvjfun.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxxdbeqy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gebkdptau.sHtML

[D05] 访问与修改元素
来源：http://baike.fanxiaobao.xyz/Article/details/gguwjqdbm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fanxiaobao.xyz/Article/details/gkmzmtwru.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhrxpmlp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gxwbrzumi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrkdvhzu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fanxiaobao.xyz/Article/details/grebzwimg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcixeplv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fanxiaobao.xyz/Article/details/gyupdvafe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvascaysw.sHtML

[D06] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gilcymsla.sHtML

Py:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gdbvuxwzm.sHtML

PHP:  count($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gceqvvcvc.sHtML

JS:   arr.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcwxjfab.sHtML

TS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxapelbex.sHtML

Java: list.size();
来源：http://baike.fanxiaobao.xyz/Article/details/gszpistlw.sHtML

Go:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgrosfwt.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gacjooxvk.sHtML

C#:   list.Count;
来源：http://read.share.fanxiaobao.xyz/Article/details/gstkqceeb.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqvprskq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fanxiaobao.xyz/Article/details/gbydhycxs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnazhxta.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gjhdwsxpt.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlhzcjxq.sHtML

Java: list.subList(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gdcvezylf.sHtML

Go:   arr[1:4]
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvmklpbo.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbfarjul.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmpsfmdo.sHtML

[D08] 合并两个数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gskdctdpe.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geactmukn.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fanxiaobao.xyz/Article/details/gwvujioib.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfjswlfi.sHtML

TS:   [...a, ...b];
来源：http://baike.fanxiaobao.xyz/Article/details/guphpdwkc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakywvmyf.sHtML

Go:   append(a, b...)
来源：http://wap.fanxiaobao.xyz/Article/details/gnegfojil.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqcjygmb.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/ghkgmhhme.sHtML

[D09] 排序（升序）
来源：http://mobile.fanxiaobao.xyz/Article/details/glnkrvoyb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdjmafbq.sHtML

PHP:  sort($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gahsctkph.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fanxiaobao.xyz/Article/details/gynxguzog.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fanxiaobao.xyz/Article/details/griddfzdd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fanxiaobao.xyz/Article/details/gebojskoy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgivhcmq.sHtML

Ruby: arr.sort
来源：http://blog.fanxiaobao.xyz/Article/details/gtnpvkasb.sHtML

C#:   list.Sort();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvtlqkvb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrglbpxa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gmvmfpuvo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyufkqrc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fanxiaobao.xyz/Article/details/giljtbsla.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrfmhyjh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fanxiaobao.xyz/Article/details/grplualhz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fanxiaobao.xyz/Article/details/gujysbsiy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnwmvyog.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fanxiaobao.xyz/Article/details/gtabzupkb.sHtML

[D11] 反转数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmakfbeg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fanxiaobao.xyz/Article/details/gqxdugppe.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gahltcqmk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxzuafli.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkdcpmqe.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfnotfxr.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcwifodb.sHtML

Ruby: arr.reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhlgbjll.sHtML

C#:   list.Reverse();
来源：http://m.share.fanxiaobao.xyz/Article/details/gogfxynhd.sHtML

[D12] 查找元素下标
来源：http://mobile.fanxiaobao.xyz/Article/details/gggcbwxos.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fanxiaobao.xyz/Article/details/giccdetsr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gtupdhvcu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gyqykfvny.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gdzndriqq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdyiapmg.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gwezhrhtw.sHtML

Ruby: arr.index(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gttipspnu.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fanxiaobao.xyz/Article/details/gruocprbl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fanxiaobao.xyz/Article/details/guugmdkki.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gbgtcscoh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzxprqqq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/ggfrfkxpc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gldoseuwh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gvtwqymes.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fanxiaobao.xyz/Article/details/gncxzblcx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fanxiaobao.xyz/Article/details/glebssrnr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatdjgrub.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fanxiaobao.xyz/Article/details/gegfbuwpj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaycdhld.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbyvmgzp.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gziozrkwt.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gfknxomsj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/glmuoowkz.sHtML

Go:   // 手写循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gckykewqy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrmevmit.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gjnrdvggr.sHtML

[D15] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduooqdar.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/guzzlyytt.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdovttmuw.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtngsykgo.sHtML


<!-- 参考信息 -->