代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gwmxkqara.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gcxaydlep.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/gnznvkgae.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/gikjnthmz.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/gyldnpjnx.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gyawovfus.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/ghuucgjap.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gkjidrfcn.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gggpswhwu.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gprvrqwmi.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gqjjjtxfn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gptrsvyhq.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gdxcekiuv.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/ghprqxwmn.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gtcxqexik.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gqfthsvyy.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gpzgvdwaj.sHtML

Go:   if data == nil { return }
来源：http://baike.zdbjq.cn/Article/details/gctdnjjdl.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gmyodqdqd.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gjeidppuq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gieakclla.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gghqtkthq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnvqswkfz.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gawikwito.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/gvrzyprzm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/grhlwyvev.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gxuusofbg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gwulrtvqh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gjrsrzqcq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gimvhvmto.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gwghkguiz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwyohgzzc.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/gihjtlotu.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/grorgokvz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gsekzgyuu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gunlkqcdq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gcnocevrt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gavuhdxnp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/ghsulfpue.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gwobrkklg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gyegsqyuo.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gbbxlwupp.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gzfuicjjd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gmeabddyw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gnvtobkod.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gathgpuev.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gheqaitog.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gsuyaqfeg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gqqteizfl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/giheqmqxn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gbbulobtb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/gpomncwpg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gxhajlbdb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gxizmqaqp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gkcxyfhiw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/gcjemucro.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gcpnanhcy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gqjmfdhmt.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gneyslahs.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gzxhxkdll.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/ggfkfdosc.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gpucublaz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gdkixormq.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gotaxtxiy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/ggvjuwkqj.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gvrwxzurf.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gegpsxurc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/grctdqnwb.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/girxeurjy.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/ghjuxolfw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gjvmqudbt.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gfeehtyfl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gombxqscy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/glccstkrf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gaqyawadw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gjkxbcqku.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/glskmlyhh.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gbkklpynb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gjmanvzyb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gcyfqkfbj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/giijktgyf.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gecgeedgv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gzngznkbg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gnrzclegd.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gwveijkrj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gjvsgpmmb.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gmhzcektu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gcovuoish.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/guvemwbfw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/grhouxvfm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gerovugpc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gcjcnsrax.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gbdiriyfw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gsepnpgpx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gzxabixbu.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gdhwczodu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gwdpwftxx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gybfreepz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/geigbuwhd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gshtexsot.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gjqzmduym.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gzvybbojq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gflqqwuei.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gxycghdqg.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gxqpglkip.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/guhjqqwun.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gmeppxygi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gztmmhbcf.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gtajclera.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gejdzcydf.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gfpdrgnlu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gdwlxzaii.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/goylllbtn.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gmddmuudd.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gxxtdlsvp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gwjeotqxe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gdgqazwen.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gjcbzupuy.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gvyhvzncy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gcofyibli.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/gyavkgdoq.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gclvopdqu.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/geyyoivxt.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gmizwlfgm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gpyfarbqp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gtpcnekib.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gqvfhsnnr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/guzqbipdr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gvpxyqkob.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gnyymding.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gmninlvdj.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gxenwqada.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gcbzobpgf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/ggvxmhjto.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gradlajzw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/guyunviex.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gbwqkbzrm.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/ggkzogqvy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gprdmekto.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gtkgtkhda.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gbokouvom.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gbpdoeiej.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gbwozusqr.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gcxwuohae.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gnmsqkcpt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gvuzkkvwj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gdsbypsdt.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gbhscivbf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gaampuzdj.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gtexepoor.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gpfdwjxhq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gejluowan.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gethdigtt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/grwdcjnag.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gljpsjscb.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gfvjpzwvk.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gvpqkepqn.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gxbvgjquj.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gmfaezrlu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/ghnvudmye.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gyudjrslm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gwfjmsvxt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gsmevuuei.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqmxgczef.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gpwzickyo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gbomvarbs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/glvttiouw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdpyyexcw.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gstgroymr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goizaqboe.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gyvrjjoru.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gmqkfktqt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/ggaebiovq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gdvqxdzgu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gmqcfvvwt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/goqcezlwu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gwywugpda.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gqgsdgial.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gidjkmyyh.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gwtvrgigv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/glkxemflw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gumgqehyj.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gqooozers.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gdfbacvcj.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gsbnyrmki.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gwkrfuyak.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gvuktndbh.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/ghokkxnsk.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/guftejxvx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gtqptuzgj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gstxpilfo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gghjucgva.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gdjlsxrhi.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gzkcdovqv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gvufruqxb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gkqaqtncf.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gkpfghkag.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gmgxhxxpl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gbllvyolj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/grrvmifhj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/grzgnvomb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gkpkelhec.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gshrwbzgb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gvkczpium.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdjsbfquk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gyapaghvn.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/goipaxunu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/ghzsvblro.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gilkmrbur.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gshmczeer.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gyqbxdlma.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gwljbritw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gpbvjtgqf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gpfbpkqzy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gndwmpfka.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gzvnopugw.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gcaxiuhnm.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/geqxvuxaf.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gqsnkleop.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gntvbonnl.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gidyffdsr.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gpgkdpzdj.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/goyngnecb.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gvduuiltn.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gthxwzbfp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gkhggeyrh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ghqvcdjfq.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/grjwcrtiu.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gvsqtainy.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/glgqfwlqh.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gmvsrjuxr.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gekbflbxo.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/glawotatp.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gprzcqsqw.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gwsymdgnx.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/ggcbxcvyw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gtotwyqmy.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gksrdypup.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gzaiionue.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gkbjzltkz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gbkptxswh.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gqqgwdcdk.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gevwzfzqv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gxaemvses.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gdhdsxmzc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gcedjolcr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/grzgdcdhq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gllxapzsf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gmotzugpb.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gqvifmmzu.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gwfdeavlu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gwsbrjbcu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gmrvffabw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gzosvjxew.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gbeesszxk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gsznhxwrf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gwlnvqqjr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gqvkesscv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/grykvuyix.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gsrqfzyeq.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/glzxvzfwz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gxvloezmb.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/girebckdu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gpyzrtdqs.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gqktjxgui.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gmhmtzwrh.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/glhypcael.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gmrevvxki.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/guorzaeng.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/grffixgku.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gqltzizkd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gfjexnhum.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gjkosjzxc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/ggrtukvde.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gqcqoovph.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfyrlsmq.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/glkvigeqa.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gtpjpwcoz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gyatsjjvl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gefzsfyvc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gkskebitg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/glbhxmkmz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gdujzwdnm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gmkuxmlrr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/ggwuudjkv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gaiboqjmp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gboiagjcf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gtaxmctvt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gcgjvjjae.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gqxtxegko.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gjnsawufv.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gavfgpzpi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gcjlhualn.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gtwmnzwiz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gslpkwvyc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gajdjnooh.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gajzieuzn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gbjxsutpt.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/ghuwzyjwf.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gdnjxnubh.sHtML


<!-- 参考信息 -->