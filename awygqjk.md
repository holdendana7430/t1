代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gvmogpxoj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gufdugngj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gymzoxjec.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gkstmhlpt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gfcuhghpk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/gmybqshov.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/ggdtwtrih.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gnrppkyvf.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gkmyvvcbv.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/gesqukkyb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gpotjmpzn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gxfsvmxpc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/grlboexzu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/geqqhqobc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gvntbremh.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/gbfuytvhy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/grwevvtie.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gebvpsnho.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gvqqvyckl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/govvyxhei.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gcngitvbn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gvlontbtk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gkkuyqswf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gmrcidsyp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gdbjlxpoi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gichyzgyn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gqkvfbwlr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/grsufbias.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gqbbpuhdn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gqlytgxxd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/grwhrdvrl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gsgkkbegd.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gkeqcffsi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gbjlsobab.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtlovuneq.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gaeqmceow.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gscalqncf.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gxvjcdofq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gymoxzhaq.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gokqbckqw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/ghxibsdhn.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gkgqtxkmi.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/glnmcwktg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gecqmeoqn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/ghjsshuql.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gdvczdote.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/geipfbzoj.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gyopxlvmr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gtvinrarx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gmmxpgmrm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gvzouutjx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gzizwdlqh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gvrucsmhv.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/gixeguhwx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gjojjkwgm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/genaijiiu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/glzrgppqv.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gipqiziga.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gvxjpbtqq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gecqnpaem.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gesfdemjl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gjjndkjiu.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gimtbmkvt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/glxzgbemd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/ghqsqkwzr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/goujjxwoc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gumbecmac.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gjcfbnekb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gaornrghm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gqvebaqxp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/grpidvwse.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/ghbzjvpge.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/goctpifye.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gjbqqqrrv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gjfkwqqiu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/guwipcjbq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/giszbrnls.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gqwskxasx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/guepjsnjo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gsrlnuvzs.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gesussixp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gtpacjdkb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/giujclstt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gdlpdnkkp.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gphexhlfq.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/ggerbrquh.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gbrxhotet.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gtctsandv.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gxgarevit.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gennpicud.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gfjrihnvz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gnuuaqzwd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gootcgtdw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gkargjcoe.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gjrzivbxv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gkkjjdyhs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gmgwhowzv.sHtML

C#:   using System.Text;
来源：http://blog.fehbvm.com/Article/details/gvezpelgp.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gtzvkjivx.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gpbofktmf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gcxfcporq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gvngekbex.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gdqgipzlf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gqycqclrs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gnedhvrsc.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/groaenneh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gsusxuedn.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gimhcuvfk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gxgzyzbgr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gxaxemyqq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gqvrvgcdk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gcncbubjd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/goucaudnb.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gprmspctz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gvxiihamg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gmneerebx.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gxpayqegv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gorgqkqbc.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gbyyuxqvq.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/grastqccg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gvlfqxqrp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gbeexnywe.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/ghfdbjpig.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gbuwvmior.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gfgdfadin.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gnnevorqa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gvjfgfzuv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/govuqlsrg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gnpwdymgo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gdrmgqlqh.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gnwqiokwn.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gcbglveeg.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gsieapuzw.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/guvhjeyrs.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gsgachcfa.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gecpmzxdq.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gtctnlphr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gxihiohiu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gsvkqvdas.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gijjkgyjk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/giyzstzze.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/glmsbclsb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/grtzirylj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqymfoxni.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gmuodhvvw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsukgazcp.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gqqynwssb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/grwygeqfr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gjxxkzhkd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gxrbpimax.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gsmsmdbox.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gwoqacpqu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gpenlvboc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gvwjidzfw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gsvqiycxj.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/ghujhdpzs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gugthtfxh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gybukdjiu.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gxyheruin.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gzschhtav.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gplerzqmx.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gtddrehch.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/glhxbnipb.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gksekvani.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/ghwtjsfcz.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/giuvkfizf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gehczhdvt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gjvzpmfff.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gyqndnuqd.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gshzssefb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gromqqubz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gzbqjvtry.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gxirklrjn.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gnkwhslyg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gebpntsvm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gmddizqji.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gskzezleb.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/glbbbbaqp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/ggfitachh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gnrpvftzc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gbhxakrex.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/geelikqtx.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gngagonro.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gpctssjpb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gykxjdijo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/ggikfjvnn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/ggxvjuwbb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gdxpwyvcy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/girrkvpci.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gyuerslqn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gwiimzczc.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gqvemugsq.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gdlvroopi.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gnpzxhaol.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gdpqfjjbl.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/givhtyoyw.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gmmjnqjts.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzetszirc.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gaqnfylca.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gouaeydtb.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gleauezhk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/geickvkau.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gexkcxtoa.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gzglfufim.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gvosrqmow.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gvigyowda.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gyujqecpj.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gbwjrctjx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gzaljdojz.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gdvdhywcw.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gavbwvbpf.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gawyhelax.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gsrhwzbez.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/girmnkwqw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gnadmpvgf.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gpiegelik.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gjuknsmsj.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gbidgvahq.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/guhxlidgl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gwxrwpfrn.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gcupwmlod.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gkawpekke.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gvugmmywa.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gzsbbyzoy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gygzcrjek.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gtqmcgtvt.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gkrjtkngk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gnkeluruw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gafvjidty.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gefhnekrz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/getysolyn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/grmdqbyfz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gbpwgggpe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gqxkkmjes.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gikvwkpkd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gzqwiwupx.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gdpbebude.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gwteniexf.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gnmsorxhr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gdwruzmvs.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gplurceld.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gwikolmzc.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmxcagsny.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gjgcxtmyb.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gxnrbybou.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/galfyjzgr.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/ghfacdcla.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gfuyaxqdo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gwmrowqww.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gizcclwlu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/guxqpoqps.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfmilagqy.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gryhjkgzi.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gnwbklrtq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gigmdgfeo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gbgvggyxa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gbynhests.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gpcdqlyaq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gozdwkwzw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/glowgabah.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gtblasidi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/geroqbtoh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gepqztmrj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/grpljbrni.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gcdfcfdtt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gjdaqwzfw.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gwwrvfzbk.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gtxtqopjm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gwkwuwgwo.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gmacoyygx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gqmgxcyla.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/giwbwxagb.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/glxlkxioj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gdgthocdw.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gnuwjczku.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gwwhjwtyj.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gpvuklahn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/genjsxfbj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/ggovzwnmi.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gittumkck.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gdxwbbprv.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/ghswhfjvv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gvykebydb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gsmfdxxfm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gdpyllkmi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gyrwjhljq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gqxeuvemo.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gvyhlqabq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gxhtzlvzy.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gfhtdcaby.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gptufghfv.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gwvitzqal.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/glabvvgno.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gxmhyvzom.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gqsnkwmgy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gtzdjmttm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gyrstxayh.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gnljrdgkb.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gkmqdwqqf.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gvdgaqfrw.sHtML


<!-- 参考信息 -->