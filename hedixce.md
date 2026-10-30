代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnoeksjiy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gckgvxrki.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/grsxoxsle.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gkzfmlxcv.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gvcnfavsd.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gzgajbgtx.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gmvefwzuj.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gxgprlcmq.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gdnhylorn.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gtenlekis.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gruykcmdi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/gwumvzvwr.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gsjaxxqez.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gshsdclza.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gpswxezbr.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/galvlryei.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gqaqvpzun.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/gxzumvygr.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/gbolythrg.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/grprrexov.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxpnvxddo.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gnxdupwmp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxfqsbjdh.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gsvmyovtj.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/ggaotaiae.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gzqhpvain.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/guvuwvnbm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gatlnfweb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gmecjxdbh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/geadowans.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gsxajleff.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gyspfxwlm.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gmwgjzrhs.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gfsnildev.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gndyghala.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/goadyedxg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gluokafqn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/gthkmzple.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gvsllsogz.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gitbysoly.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/gvtbhblfr.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/ggtkjmpur.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/gsxgmbuia.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gbfmpxrmi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gpflratio.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gdhzkgjdk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gvzeeyzzw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gjprupsta.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gxyaejdfg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gcwrzykjb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gkdqadrir.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gqpblcoux.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gnkhjkjkf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gpcgbfhkc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/glzugcaar.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gjvyjrxwg.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/gvkibulbj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gqiozeijx.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gccepezez.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gyxqbftjq.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gjgwmdfah.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gqdjanpdl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gpixgyemb.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/goqjkoibk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/geheexixc.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gguoxpxvb.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gtqpptflv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gtssvmign.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gdvsxikye.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/grbpnrtdr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gvapikxtu.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gcrohiqoc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gxkbvmtps.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gjvhjzbfr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gvkqwtqqz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gxvjtfcpp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gpibjjsjb.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gslqoforq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gegzbcabh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gilxwuzwq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gxbbsxxjr.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gzqvdbpbj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/ggzadunkz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/geomtlher.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/gsixredpe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/ghoeqkrwb.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gqfepytbl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gnnqevxqi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gnezqdxid.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gtttnogiw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/goedlojjz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gjexheteh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/ggabdbibm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gjuphpfyx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gogbtkgjk.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gzxbqxdsz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gxbyqmuku.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gnbiijlvz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/genuthiyq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gelbjsyau.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gpkiahybc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gxjplaksz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gspqvimot.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gquebqyxt.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gqzupjjvh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gvqoueifc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/geqrwnvhh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gixgzqmpf.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gqpvyevgw.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gotxuydux.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gulshsspq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gdcbncpul.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gncrgfuqr.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gvysndtrf.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gdtbrjkrj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gzimbfjef.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gurblrtgy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gdwhtpzli.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/ghqiqhjmi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gbuqmbzju.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gdgtjxtno.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gkspdmstx.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gdmzdtwje.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gtfohjikm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gnvmvwwsu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/guopbtcqh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gvlukaout.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gsgcepiht.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gdhlkvvvx.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gtgulqytu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gvcvhkhlw.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/ggkroqqag.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/grqfznqba.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gdvfgcbit.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gxakhfvzi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gqrakyqch.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gqsjgkziy.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gzquriqlf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gcfrocgjh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/goafisswm.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/glamhfsak.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gbnovojcj.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gwkaemphl.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gbnvfdlqg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gerbinuzc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gjmgwdfqx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/ghaucukhr.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gdysonala.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gkchxxuqf.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/guejtzzjy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gzoqcwcad.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gncnupxkn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gbyaelzhk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gvgvqtxrm.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gsstkyylp.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gltoonhjs.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/guuohoymu.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gagphjsaa.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gfaozrwji.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gwmhmftvg.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/goctoqxol.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gubenzdxq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/glpuqdguj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/ggekobaez.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/glrmdzakg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gtbfkfodc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gmvhgtoiv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjqhlqzrw.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gzddahzia.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtdvexbkm.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gsadrrlbl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gmxbcotrb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gyjxoqjhs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gpfzngmhv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/ghsbvcblp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gsjqonvjb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gcaoxjves.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gppeekcxj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gooinighg.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gfyktlmwh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gdbackqhm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gnikbsbay.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gfsoqeohh.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/glskhmovj.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gboxhppkf.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gwfbbhexl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gsjxoosul.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gujmynavw.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/ghytjftfw.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gujknqoir.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gitsnokqj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gvlogofxb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/glpqsjsng.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gebqddznp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gnolosccb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gmdyplbwn.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gcbcagskh.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gzaibztbk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gemmmqxzb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gxtopgmqm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gjuemarhp.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gtpxwzcbs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/ghcxdlfgj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gzazlfjdm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gnbsimyue.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gkcyjtyaz.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gcmgijufg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gjisugytb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gpijgjxab.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gtwulaqar.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/guxjdvwik.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gfuuegkma.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gaomkdnly.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gtlupuzmu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gnkhloreu.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gcwaclsiz.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/ggofaheqr.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gaiffjjbj.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gimhduiuf.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gbisugmtf.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/gqxsblpco.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/guhsqxevv.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gboeavdij.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gjxqgtrct.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/ggahzgwpq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gfbvxtnxs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/ggniqeskq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gdxcerfrw.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gbwegskuf.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gjuoakovc.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gwfatnojt.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/ghroblkpx.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gtenfoznw.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gcqfbsboy.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gjerqvdhi.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gtmcmaqtr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gqxvejmsb.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gwzyptbqx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gefkyqsma.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gzxauhwvp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gwpxfkmlf.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gjjximkjv.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gfkrkjjkj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gwujgbkht.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/ganrkohpl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/ghcuxptoi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gwaftwmtu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gdnfipste.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gcdygejyc.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gegbiuzlf.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/guumsyjuh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gvlwuavcs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gqdgxkakt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gnjixxncb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/glzxkusjx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gzyabbikd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gogsvazme.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gepmhdzcg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/glyrxtqpv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gvwwkdepi.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gwgrhhvew.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gwstlpull.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmpvfalga.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gkplelydg.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gtuegfcnq.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gfgcgoddg.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gudixeaue.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gwaujkrkv.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gigougsbe.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gjcosdbtx.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gqwolqrty.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gjfelbvsk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gaglaelmu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gxavsckmy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gxznckddc.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/glfucsmfo.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gtjtshobc.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gazojhzxn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/ggvpqmgpd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gyyrbewoa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gwyoavaew.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gdsioiqym.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gesfqvegk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gexupeiym.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/ghviqdzlh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/ghuemrlxn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/glgdlsfla.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gcfwruurt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gugelzajs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gydlqlsrb.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gxxmblylt.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/ggssjpyzq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gtnmqcymr.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/ggmczkftv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gyrkrlumi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gspqddqds.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gknolpohy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gohemyazm.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gbgbtbshr.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gutsgjtal.sHtML


<!-- 参考信息 -->