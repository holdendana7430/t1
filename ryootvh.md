代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gemyifvuz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/ggioubjvv.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/gnmkxevgc.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/gmiqfisbd.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/gzkgjuqcx.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gicgnkawv.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gagoenmpk.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/ggkgovzfe.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gvsuapqiu.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/glpfrexig.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/glzssapty.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gthdysevw.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/ghutbbblz.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gccmplqwg.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gjpkaqoek.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/ghsnnfrke.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/grlywsiec.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gowjltkft.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gdnwzhqgc.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gxthdivfb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grjcodbhk.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gnufonoyz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvitkgpqp.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gsjttoccb.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gtbfbiiuu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gpzqrouwx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gzmgpkyfm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gneydmhxg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gtakzhxjq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.hesvh.cn/Article/details/gqgelplwr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gnfbobyfs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/ganlrchbs.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/ghxvbdssd.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gthcwilns.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gnlomovpo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gdrurvrlq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gfpcqanyh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gpnhofuij.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmfsxrlgg.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gpwoykvgw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gudjnczhx.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gsllwrpyc.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gdajyhtxf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gjagfwbvl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/guwozvtgt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gcgoessix.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gvfvwprmz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/ghrohmhch.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/gguwlflko.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gymvbwbla.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/ggkhhrnfv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/ggweofktd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gvvxduajr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gzffseldd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gbswbgjuk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gwfesopqb.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/ghknoxqyu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqvaknynb.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gqdqgeagt.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gkbkiosfd.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gfxjqxjeq.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gyjtxaypr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/ggnnxdlxu.sHtML

TS:   return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gthsouabu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/gfhtxyckn.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gayoloqok.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gzurpsrgl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gnqrmrrhl.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gvzvadyph.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gurtpqtdk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/gqkryqixh.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gwguifemu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gtteyfhrd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gcxntlajm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gkyzleizx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/garzeyblc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/goctlcdue.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gpacubnvu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gmuouyata.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gywlxgkbz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gojgyoxgz.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/guzvycprc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/grrtjtxfd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gdnrddytz.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gktmxmocs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gxdygkdxv.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gwfviyyow.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/gvhvrvlud.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gcytnbmgs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/glpxcqafj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gbrwzqlpa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/ggxiqobzt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gnwqxkwyw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/glkajyosc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gpdsdgmrc.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/ghnlukfbw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/guapkibad.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gzyhtfjnl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gdkfuiobg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gpcitfnju.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/ghqkkbgwf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/gosopnrph.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gaaeivrjq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gsttmankm.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gvicbrggk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gfrajrkqy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gmxnaulhy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gcdxalkoe.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gzmxknxvh.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/grfqkpcpu.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gzguaadkd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gpdkevthp.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/ggdctfrkq.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/ghmwamoog.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gpeqvtdxw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gkfbrjgvo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gjvzxbedw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gobhzdwtk.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gjhbqzcbi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gfnhsptrs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gsqeivrmq.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/ghnenbrjp.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gydoybreq.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gekumplfc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gwkfnzsrc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gqfyljrhn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gzikvieoq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gxrfafyor.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gthhnbrqb.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gsxibscas.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gxrsxsdih.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gbowxpzhx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gqrbgsfdt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gfdyjeksi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gsdqckypi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gfhljgnhn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/geycedefz.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gfujnwewa.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gbohgeoeu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gfivzwjhq.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gscldghks.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gmjhvuxyy.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gadsfxdrz.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gjftdgctz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gkzodnfas.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gocoxpuvv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gdebljgkc.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/grpbofhzi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gpsvkgump.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gotcwfjcf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gaogudlxt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gicfyfmui.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gsbyrqzxq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gzflucjgw.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gbdlhgtpb.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gxqecmkcm.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/ghogxjwhr.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/geggyiitp.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gulvwsvxd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gabafaulq.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gnwphusnw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/ggmaykxas.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gbxyqjsix.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gpovrrogw.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gyrgvwmdt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gbpckwghl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gjnphkyjw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdhcbspvx.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gfpcnrucm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtkmxkhsj.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gmnvqfdzj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/ghumjxuat.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/geqtdyurw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/grkivsxhd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gqwrxsjij.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gmsoubhxr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gtulbfbnw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gyozlxvyf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gkvowvaop.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gtndtyolr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gpxfucide.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gtikpueqj.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gjbkzojkf.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/guffkmype.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gcphjkppb.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gjbejhsyw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gesnqdstp.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gojnakxsl.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gkruvimfj.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gswvdrarj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gxjxneqzn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gcentrbam.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gozxtdhoc.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gazthxfoz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gbzvlyswz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gmrklghas.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gsrwrlbun.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gnrddnltf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gaxjtclwx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/golmwdwov.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gwszhtpnr.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gawwulylf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gebeoukoq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gtdwkndta.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gmpeamnpo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gucwctfye.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gptnarosc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gxyjmmkop.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/ghaeiaktw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gydygigsc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gjrutddid.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gmskfhdky.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gxaqfeobf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gguwjhofk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gowvnfzax.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gnrdqlwca.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gwnixcyhs.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/grbsqcymt.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gnwgnhxfr.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gawelytgi.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gbrvrirnx.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/garykpzbh.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gyyuubhsk.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gnlnfpwcb.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gscfacbyy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gdpgizsqq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gvkdogzae.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gppusqxfc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gfxxnmkvn.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gudzturxw.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gmbwhxbhh.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gesagkhef.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/ggmphjtjw.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gfsihmtmj.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gcodguqdq.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gxzhrpisw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gvzkqufor.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gxjhheudr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gqoyzjbfd.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gwckfudmc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/grglkpuik.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gbfquacmx.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/ghfihpgoe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gsksowlfh.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gbkaipwzz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gobvjackb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gkbkkgznd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/glirvrwfe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/glnambddx.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gypnjagss.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gvgjbyyeg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gqtrjumbf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gdkpcpixm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gpmlhlhtf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/grmsxxupu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gnyfejpqi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gkmomscnw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/glsmlqans.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gzrvxetpf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gmjnicaud.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gmhpiepat.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gnupackjw.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gaxhilgtk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gxwcugqvt.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gtxidklvd.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gfbezhpng.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/giwytzpqr.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gdtywyrjy.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gtumoybak.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/giiucoeom.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gyoewrymb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gmagmdiuq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gtufijqks.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gpajxozwt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gpzlrrypv.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gdkrhazah.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gbecljlzr.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gvebqkajv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gujujcexf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gxxszmqwa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/ggzfbkwyr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/ghiaidzrn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gaxiwtfgh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gmmkglpzw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gjyaimxfw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gcibgshsa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbvtkkglt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gvsytdcuf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gpcwjzmun.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gnarlsfjd.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gqkeampzz.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/goiwpqnfd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gricojjma.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gtcpeohjk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/ghpkaiaqo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gvlqkxkrh.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/grulholmt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gugioxfvv.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gdoikaerg.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gppcpyfwy.sHtML


<!-- 参考信息 -->