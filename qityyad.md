代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gfhfbqhuy.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/glceoewjw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gdooztlfb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gfbjzzdce.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gkagbaivv.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/gutpwunrn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/gthczfbda.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gaavqcuvx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqziovrbc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gxdnxzqbu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.hesvh.cn/Article/details/gmgxitihd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/ghjkeugkl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gthfxbksl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/ggbkjeeqn.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gxzoienav.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/ggmfobuis.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gzmlafuew.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gpfztfypi.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gqxosboct.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gqnsbjxbl.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gjxwlqgqf.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gddavdxki.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gdbrqorkc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gifeqzjtw.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gvcarwpbq.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gwtmcohoc.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/glodrmfuy.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gbrtppxat.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gxlqggoar.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gfmhmidua.sHtML

Ruby: return if data.nil?
来源：http://wap.fehbvm.com/Article/details/getzwscwi.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gogztinvh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjvgyriio.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gbimntmfg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsgtwzyfh.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/grdqvwfhl.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/guwfljypt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gfzmyieai.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gmcfkudoh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gzjuhluxv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gbktdsxja.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gfhcfhqwt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/griludzks.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/giqfvftct.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gragonmim.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gcvxikmsm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gffknzoth.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gzwomrxfs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gadowiacn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/gqwniuwld.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gbvdbehcj.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gforfvelh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/geymtxybm.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gaeecdrfc.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gzggdlphh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gbsvobako.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/grcexokzv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gfrierenk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/gszglimvq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gitwfcisi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gkxfmaucf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gujdbearv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gznjycyxu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gyqyuuddj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gpqgbaekd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gljfgamcf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gjnujcvuf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/giorddyre.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gisqlizif.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gwlvxvlsl.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/grlbtkqea.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gljdzndwt.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gzvlaqamb.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gecljluql.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gjusbmrwb.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gpmpkgzyw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gjwxfslzu.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gurjkhehd.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gqhebypjr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gdmquhahx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gzbmricif.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gtaihtcmd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gdddfwhhl.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gkvocckqh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/ghialaisv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gkjltzbfn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gukltrlkw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gtqukdvvz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gdbpfaemu.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gzlkizlgi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/gnbuutrso.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gniekshsr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/gipmdakti.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/ghwotccny.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gaxwsasza.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gknltmoqb.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gpkuzpfks.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gschwonwb.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gbuykvlyg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/ggnyaevuh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gnxdmvibq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/ggnwrvcsw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gjzuegsen.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gukvnqppa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gmknpzbrd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/glmcfmodx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gzhgjledg.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gxeywlqdx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqxghnzeo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/glejqjnzt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gssdjqtjw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gvmthngir.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/glenlgtrv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gumpiachj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gfqcjcidc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gfghuzchx.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gqdfaxeuw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gwbpvzjyy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gwdilezpl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gwoqrlyzi.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gdrgyspsh.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/grjwscrhv.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gziwvkaih.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/grlvvghxr.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/griwebgub.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gkyvdpexx.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gzlttusyq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/grzdzcjqz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gbmvfptjd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gjfgfswcx.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gvsuvvqhf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gjtmkrccb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gpefyendm.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gobjotgrm.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gxwjcaayd.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/girvagfrn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/grvjsijqn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gvgwrgajf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gatvxqlhn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gcymbsynh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gnzjjvfiy.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gslblcgib.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gtnxpiamv.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/ghagzyvhu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gidbboymw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gfubliqac.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/ghzdjcnoo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gkpupsirx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gklwtrpyy.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gxvvfzvmy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gupaehheh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gefmmyemz.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gzbliyklz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gqktkbfnl.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gfnturqfn.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/guefdovrk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/grwtfzrbq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/grlbooacs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gcwwfmeij.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/glbprddgx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/ggyfuvuqk.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/grrpfmcts.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/gzsgppksg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gsqiynmhb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gulclqipc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/glgnmdqpp.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/ggcthrbfm.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gylgutxhe.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gxrdbfmgn.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gncgdaxzo.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gilrmhjgh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gksdjjzkt.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gjtfowsiu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gfovaosqr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gdwhzkppf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gzkizmlwk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/glvlookqt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gakynnsfo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gfjpwrdiz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdbdglsnh.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gukwrbtgb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmduzjtzj.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gkipxsadz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gpijbmxem.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gevgyspnz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gqxnhsvhc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/guvruewdj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gtlgdgsdp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/ghnsmfirh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gbgtaezop.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gobrvsrff.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/ggbdfrhjl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gguntimws.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gcubydyzp.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gjfbyxabl.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gdthpqxgv.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gdnhjcmje.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/giwmtpbmw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/ghfcdpefl.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gnvlblthb.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gnhxrfizr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ggutpkqbq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/glfvaynqj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gcwcpangg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gdjvmjsmf.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gnbeitjll.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gqjoibkja.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gpolxjxnz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gukjuihlb.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gcprvpcre.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gxoykxilg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gttnmzild.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gvgleegie.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gtvyczrwi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gyjypzcps.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gwhjpstax.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gakzhjtby.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gekkvingk.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gvryswcdp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gsckkkwwd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gjtrzujkc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gtlftgkxb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gunfglnhk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gcajysxbs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/ggrpaepdh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gkoeqikix.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gswcjuect.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gwhtdmdnz.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gbsrocpoo.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gqsvwsutz.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gqjepneym.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gypuhtane.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/ggthwzyvo.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gscsggxab.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gijrduaaz.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gabkgqhry.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/goqvosevi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gislbkrgl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/girredidz.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gtnwhrlaf.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gepllwtts.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gunyjckkd.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gtrqvqpog.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gvlfhufdn.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gsmufthdt.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/ggatmailg.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gdlymvaly.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gzcqjhqxa.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gupvhwqto.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gbsaagprx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gypeduxud.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gdqpuoovn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gkazncqls.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gijozkiqp.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/glwizdowf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gchwsmtfc.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gahbhkofo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gmrtmuspi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gcgdhjrob.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gwjbsotvx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gqjzxkfmm.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/ggxngqpav.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/grrfldjxr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gwxqtksjv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gdokdkvpf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/ghahwlgeo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gnkmtbyto.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gyvjrywaq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gsmocoyqy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gmyomboyt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gtjpbzciq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gfrejklso.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gdwazhfdz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gbgciziim.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/giqardqdc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gpnncstpx.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gkuwrrzvm.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gkouikjsk.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gdxnzamuu.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gvoakxhlw.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gxokiyeuv.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/glwkcxdpf.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gdnzmnphw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvsuxlhbq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxwhihkma.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gocmlscmg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gjhnzfeaj.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gpuqcdkpm.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/glqhmchre.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/ggalbevgo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gwdjcgoqp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/goaavsvov.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/grqrlzoli.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gyhwpxrls.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gzhsatapw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gazqrstma.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gvtfwjrrt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gtwuiriwc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/ggwhjttgp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/glphabqya.sHtML


<!-- 参考信息 -->