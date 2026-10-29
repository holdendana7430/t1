代发 wailian999

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gkezjreon.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/geqsdfesd.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/guqdmosrs.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gzjztmnqe.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmxtimuwb.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gggcfqono.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggsmapxwe.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gylzrtdjg.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/gbggzjnnf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gzigbakde.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/guwmepjhu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gxdicseln.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gxxcoprqf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gldbhkxzy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gpijisofk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gehlcldqf.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/goobqvguw.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gruqqmybz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gmxvbhjxt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ggawuwicz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gyhiztobr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/gxtpuglvc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gjyqkhixq.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/goxulfgup.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gslxgwuzv.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gfcgwshox.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/gnmzmxjuo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gzshlefzz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/grqvpyblm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gsdhuljgl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/ggogtfrah.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/guhniabap.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/ghuhgtsvi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gxpephgtw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/guxmkdiew.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gkujlyibv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gntjlfwtd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/grcyhhcbc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/gmzudeqhf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gfpmlxdwj.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gqkpiylnz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gmcqegkfp.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gjfztqjfw.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gkazgjryg.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/geznacqwt.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gwtbubafh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/gwdpotyyy.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gzifyvnjs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/guvqnkvik.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gzjayfmot.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/grbgpsjps.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/gsrhpqcvx.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gtwvhpwuq.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gikbagwuc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/guilqgmxy.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gsnmdswwh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gykmpwtqb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gzzsztrtl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gqimjticp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gjmegxwdg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/grmjrbvnn.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/glyeoxktf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/glrbhxtde.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gziwlhxie.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gqvumikml.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gzdmktxlm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gnhbkfimd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gzodzsoju.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gikkflswu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gddovsngz.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gbzkyhmwn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gsywukqph.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gslxyajyo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/givywbdty.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/guvymiuoc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gawmtezdg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gbmqikpbg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gybzpkzio.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gsmxbipsk.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gtdrkleqo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/grduhhwcb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gebbwpbst.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/glfdgqddf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gcqitabjs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gvptiyjwh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gsejcoijd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gtsffyuiw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gnttzqdiu.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gnvyafska.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gswazbxfz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gznmjbjit.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gouoielbs.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gmgifqrxh.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/grjukkgmt.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gdfgtzlkd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gkiqxcncu.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gdefhfzmg.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gpojsulan.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gxdufxrqn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gnazezqnl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gufthvozj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gtwpwmrlr.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gvissfgdb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/ggauzeduo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gxeqafwpj.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/glqrmkmob.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/ggcjgfhss.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gptqshrug.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gtygmlabf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gocemvbpa.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gysskwrxa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gdaiqrybq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gcujuozwz.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gqwnbnfgv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gatfqwlhu.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gceqhjukm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gckjdvdua.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gyoigoasv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/ghzaelwix.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gktpjoixy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/grcykwath.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gghuytcyw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gzryfacqc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gpwysdzsg.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gzdybetxb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gvwiwbuzg.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gezckypfr.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gpwbzrtgv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/grzxkljha.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/geyhgcrtg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gnycggywh.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/godkywrfm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/glbgpknpy.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/grrslphrm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gujvlckcb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gyjfkbofc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gcywububz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/ggqnfkihv.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gvfkdgkyg.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gctnoywcs.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gbfgpmwdz.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gvtkdqzcf.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/geixumbuk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gxxdvrvez.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gdphbjkri.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gifbrrrvo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gdoobfsee.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gzglykjem.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gdjzpckdm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gkpwpqkom.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/ghervixyd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/goipjioxq.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gajjhouef.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvbozujli.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gcbcyqsur.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gswmudomx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/ggykjdevy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gzfhbvriz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gvycrcduc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/glbpjmhwt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gtfxqltrh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gkgekxtev.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gdyaizuwo.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gkcgnhmlp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gjvubuwwb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gqbqndtlr.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/grapxyecu.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gmgcbiyrt.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/ggywznfut.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gdjmhtbow.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gtwhqammq.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gnbzdtvsl.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gobonaocy.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/geywbejke.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gtvcatknv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gybkghscj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gnsedyqmn.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gcjlifnjj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gaomonxgx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gbmckrobv.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gxgnqcgab.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gykrncuxi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gbvfnpwxq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gghihhpyn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gtxxwmowq.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gjqtlamly.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gubsvibdq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gszduqmss.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gafcoexpl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/ghszcjupp.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gtfbvqddq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gdzdfaouc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gratrvusk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gifrpxjye.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/guthdjyxe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/ggfoqpall.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gdylloasr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/ggtuggpbn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/ggvkayqbf.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gbrlearir.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/grlectmsw.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/giabjeebm.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gmisbfhgs.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gjafhibqf.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gscqyhnmr.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gnoybpicp.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/ghzqbsnho.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gnemqzpmp.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gcqqvnyww.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gjiyoavbu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gbllhhgne.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gpozflsyj.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gtdmrntgz.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/ghsfuajlh.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gdlqmuhrm.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gsfcrfcmr.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gupqwuodr.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gfjpikuwq.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gehxqczeu.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gfwljyltk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gdsgdigsu.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gmeahxrqf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gbswuxnsc.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gzekiisko.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gsghxckdb.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gtreudefv.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gjrswpazf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gksvvekaj.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gmcogldrh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gixbzbruh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gjnwaggee.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gngktusej.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gnkmjlatc.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gylgqfzcx.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gotcbdvdi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gzkabmpzq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gaghdgzyx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gxkbdpsrc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gknpkgbcv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gcpmtistu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gbydauhvf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gtcounpvz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/grooiondu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/glqzptbrm.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/geayienzl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gatcdxkhg.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gcajyfzcl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gwfimavdy.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gzmzszepc.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gupwtjqrh.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/grjvhwftk.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gtgzovzmu.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gilsrapfw.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gtsbuilzz.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gdtonipsf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gywnlsdxd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/guluvftzr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gqwjchnhs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gxagvtocj.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gvbtotgpo.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gmwwuxdzj.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gkemkjlto.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gkcpnolws.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gxohvzyie.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/geydapxfc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gqajdaisk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gryrrxwif.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gudwobjgk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gkoodiycn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gwiqfbbcc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/geothnvhi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/glkwpbalv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gdkmxeuzu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gsfiegwpe.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gwavarxmn.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gcetqtjao.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gjubksupf.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gheodvmqk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gpcugiomj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gbzszanjb.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/ghvuvixws.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gvcvyflen.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtyiyuoul.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gcqkhwwpb.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gacnraenj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gqcylpjqs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gauviieqz.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gxtwwctne.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gdfbsgouz.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gknrpxvtp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/guaxikfbr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gtlunwnds.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gsvkebvms.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gywscrseo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/glmnsgfmv.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gjkqtxera.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gaqatbcci.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/ggvzazsgn.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gobdsiygj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfnookdlm.sHtML


<!-- 参考信息 -->