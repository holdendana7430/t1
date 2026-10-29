代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/grvivaesc.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gqtapizeh.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gjvkpvgdh.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gbtlbvxlr.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gyvaawzgw.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gphfmgzof.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/glwdebfrg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gnkeipbuj.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gfxbgmnhv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gibnkpgeh.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gwhzhjecm.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gudpiwebc.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gvdoeognm.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gwsdjnsmu.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gqtckkwzy.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gprilkezc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbgpudkjh.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/glgpgbpjt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gisqvmunq.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmizaqkgr.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/guftjlape.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gfmqvhhmo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gdegdimio.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gocmjgfqs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gnpavmrgg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/ghoqmsgxb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gjdvdhulc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gfnisxqvy.sHtML

[C02] 默认参数
来源：http://read.share.zdbjq.cn/Article/details/gmyljerry.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/gtwsdywqg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/glaeyopzb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gbkbtyapa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gsubmpeue.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gnikknkbn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gvnramsbr.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gbwnssebz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/gtgknjzyz.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/gndxwcgop.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/gilhzngav.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gzslhhtsu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gfgzysnlx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gxjuraasy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/ggwehtlor.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gzprdevwm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gjwhmhkug.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gudighmuq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gdxjvazlc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gftvmdpbl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gflvdofve.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/glpgijtwb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gxjbtdwdw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gceeimexs.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/gwgubzesa.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/ggbdpjyzp.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gydzusunc.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/gvoywvpuk.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gqxvqshrf.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/globpvelz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/guhgbttcr.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gnpakijal.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/gfpiivttd.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gmdpgrtex.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gfqifyjun.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/ggimuvebh.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/ggosycyfl.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gxmysoxoo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gyvyjldea.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gqirbqmrr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/glmaxxaro.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gssymlwsn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gghoibdbf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gsiwjlgwe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gcwgpndwp.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/gpbyzlggv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gbyueayex.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gwaavpyto.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gjwadyulw.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gdiopnaie.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gjjzznmyh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gkwjlwxza.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gutzotpho.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gehzyilok.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gmbdjbvod.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/gouehogpb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gxkkmxyyb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gttkltfjy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gthajaepr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gootzdyoz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gbdfmsukj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/ghuaxddul.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gzuvqmafr.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gailkjvql.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqyyyqdgd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gujkgucsq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gjmosjrhw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/glnueggkt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gtehusbzx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gredazjfv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gezxogwjt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gkpcslxgg.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gpljidxog.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gcrtvdhek.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/glprvodwi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gtbtupjpa.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gjpjbvloa.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gbavxizgz.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gynhavvdn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gfkougguy.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gffjrqbtr.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gprhyawvy.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gocccodan.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gxtpuozox.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/ggqlqprus.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gpudkatsc.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gtmbpljlr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gdyvkjvrs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gxbuymutk.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gsadhjzvu.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/ggjycxnzz.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/ghbtvlovq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gmpzpecci.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gfrkhhjff.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gobotskan.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gfgbydhue.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/ggerpshvi.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/grlezvcya.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gsekasyal.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/goklnzpui.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gixaqsqpf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gvibzbcku.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/giznpdguy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gnxazuefg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gtixqjbro.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/geobdehwx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gmuhrposn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/goshqrymi.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gdctvbjxv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gugdgzvxz.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gagpcdfdp.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/glamavkap.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gfzapqlov.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gvtngyvml.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gwksubyzq.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/getobctvc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gzvykjdps.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gouitolgf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/geisidrxs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gjqkxhpwt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/glwjceauz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gxmdokeql.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gjybqunks.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gefautapp.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gskgaxtvp.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gudhyjlyo.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gjjvmjlsh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gazdybwzr.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gefabhmsz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gdppuwxej.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gcbmldwln.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gztkignsf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gzcemttwz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gdeayyccv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/ghcecohnf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcqoumoin.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gcoolowrd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gggluuudp.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gvjaqhvmw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gggjizafd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gifvbnokk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gyhhetilz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gwkshbxyq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gwwahekwl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gcstjwjwe.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/grvcyfmkw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gcoqbumus.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gjwiwptws.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/giqczrukw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gwazttsjw.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gpzykpiyf.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gfrzmnnbj.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gnwbunndb.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gqfymtdwc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gjozclwco.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gsjzuebcm.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gkyucscxd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/ggyeqmuny.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gpisholdn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gdsavyqaf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gozpfeggi.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/glniovytu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gvniznvnz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gqvgmtgcx.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gboosjpbx.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gjukhevcw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/grzikxlvn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/geuhhaktn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gxuipuvdo.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gesugaczt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gexmdrskj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gatnakjjl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gnqgyuhba.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gjrbiywss.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/giopmiyij.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/guzbdgufv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/giarmxtuz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gpznhjwbz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gfmjvtbrd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gcxngcqlb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gjowqfipm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/ghjhytxbg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gxhdtuzmp.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gwbksvjwg.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmwztgzyr.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzwbvbyqa.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gbwoxciap.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/glchmcllw.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gqzwidgox.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gxexfafbf.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gxltcrzuj.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gkbspvbsy.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/ggnnhwvwa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/givxjjsdh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gfirojymr.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gtezmqjqc.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gslbxgyay.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gqvomqbpk.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gsicowsro.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gnqztgvjs.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gjzutjbug.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gmagfhiwj.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/ggtwivcmj.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/giphoxpxv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gyvmquiif.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/geomhjseq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/geloowkrm.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gpktocklr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gvrbdggiy.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gtwkboocs.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gdoysjnty.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gwjwqudmn.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gzobxmttw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gbctxbsmy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gzkcydmbp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/guftyjmoi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gvvavqpyy.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gdnoscfsx.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gkltmjelx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/ghwmrionh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gebzeqenq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gdchhzaja.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gtkiqvbte.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gcijxbgdv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gwxcpopcu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gsprrhnng.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gzfjgdfhd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gzeztknkd.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gxpuschue.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/grfpdwkvp.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gjpdqtbbl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gcbgovrhk.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gmekcrnxl.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gkhkgbldq.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gnzddnjiw.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gbbaeezyx.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gsederaez.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gpvdhtnpf.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gthqwjvfh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gqidcyygw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gsemkwbng.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gkbgrjaer.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gquodfymw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gsikcdmuj.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gurdpuhpn.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gvyqpfqtv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gxbnpezae.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/goghisicy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gzfsloztj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gfmtsprzb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gshryedqz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/grkuxolnl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gjeffwfgs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gsykoyfjk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gmgfdojdf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gvuvdtwrn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gmgvczjzf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/glphthkfh.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gtvmfrqcj.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gipvfrqxf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gbffvnijf.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gzkgwilkp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gqsmbkjdo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gmpvqlxxq.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/ghunhdjal.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gtwflwuaj.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gcruntiac.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gyfbzcvkn.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gpihnkqul.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gbxxaygjt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gsixcxjrf.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gezdhqmjf.sHtML


<!-- 参考信息 -->